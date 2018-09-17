<?php
use Drupal\Core\Form\FormStateInterface;
use Drupal\Core\Theme\ThemeSettings;
use Drupal\system\Form\ThemeSettingsForm;
use Drupal\Core\Form;

function pivot_form_system_theme_settings_alter(&$form, Drupal\Core\Form\FormStateInterface $form_state) {
  $form['st_settings'] = array(
        '#type' => 'fieldset',
        '#title' => t('Pivot Theme Settings'),
        '#collapsible' => true,
        '#collapsed' => true,
    );
  
  // Color
  $form['st_settings']['tabs']['them_color_config'] = array(
    '#type' => 'fieldset',
    '#title' => t('Color setting'),
    '#collapsible' => TRUE,
    '#collapsed' => TRUE,
  );
  
  $form['st_settings']['tabs']['them_color_config']['theme_color'] = array(
    '#type' => 'select',
    '#title' => t('Color'),
    '#default_value' => theme_get_setting('theme_color'),
    '#options'  => array(
        'default'           => t('Default'),
        'aqua'              => t('Aqua'),
        'cedar'             => t('Cedar'),
        'charcoal'           => t('Charcoal'),
        'greensea'       => t('Greensea'),
        'red'            => t('Red'),
        'serpent'            => t('Serpent'),
        'tangerine'             => t('Tangerine'),
        'yeller'           => t('Yeller')
    ),
  );
  
}

